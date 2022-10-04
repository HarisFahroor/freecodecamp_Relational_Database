--
-- PostgreSQL database dump
--

-- Dumped from database version 12.9 (Ubuntu 12.9-2.pgdg20.04+1)
-- Dumped by pg_dump version 12.9 (Ubuntu 12.9-2.pgdg20.04+1)

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

DROP DATABASE universe;
--
-- Name: universe; Type: DATABASE; Schema: -; Owner: freecodecamp
--

CREATE DATABASE universe WITH TEMPLATE = template0 ENCODING = 'UTF8' LC_COLLATE = 'C.UTF-8' LC_CTYPE = 'C.UTF-8';


ALTER DATABASE universe OWNER TO freecodecamp;

\connect universe

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

SET default_tablespace = '';

SET default_table_access_method = heap;

--
-- Name: galaxy; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.galaxy (
    name character varying(20),
    galaxy_id character varying(20) NOT NULL,
    size integer NOT NULL,
    light boolean NOT NULL,
    has_life text,
    far integer,
    range integer
);


ALTER TABLE public.galaxy OWNER TO freecodecamp;

--
-- Name: moon; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.moon (
    name character varying(20),
    planet_id character varying(20),
    moon_id character varying(20) NOT NULL,
    far integer NOT NULL,
    light boolean NOT NULL,
    has_life text,
    size integer,
    range integer
);


ALTER TABLE public.moon OWNER TO freecodecamp;

--
-- Name: organism; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.organism (
    name character varying(20),
    organism_id character varying(20) NOT NULL,
    moon_id character varying(20) NOT NULL,
    far integer,
    size integer
);


ALTER TABLE public.organism OWNER TO freecodecamp;

--
-- Name: planet; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.planet (
    name character varying(20),
    star_id character varying(20),
    planet_id character varying(20) NOT NULL,
    light boolean NOT NULL,
    has_life text,
    far integer,
    size integer
);


ALTER TABLE public.planet OWNER TO freecodecamp;

--
-- Name: star; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.star (
    name character varying(20),
    galaxy_id character varying(20) NOT NULL,
    star_id character varying(20) NOT NULL,
    light boolean NOT NULL,
    has_life text,
    total numeric,
    far integer,
    size integer
);


ALTER TABLE public.star OWNER TO freecodecamp;

--
-- Data for Name: galaxy; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.galaxy VALUES ('A', '1', 1, true, 'A', 1, 1);
INSERT INTO public.galaxy VALUES ('B', '2', 2, true, 'B', 2, 2);
INSERT INTO public.galaxy VALUES ('C', '3', 3, true, 'C', 3, 3);
INSERT INTO public.galaxy VALUES ('D', '4', 4, true, 'D', 4, 4);
INSERT INTO public.galaxy VALUES ('E', '5', 5, true, 'E', 5, 5);
INSERT INTO public.galaxy VALUES ('F', '6', 6, true, 'F', 6, 6);
INSERT INTO public.galaxy VALUES ('G', '7', 7, true, 'G', 7, 7);
INSERT INTO public.galaxy VALUES ('H', '8', 8, true, 'H', 8, 8);
INSERT INTO public.galaxy VALUES ('I', '9', 9, true, 'I', 9, 9);
INSERT INTO public.galaxy VALUES ('J', '10', 10, true, 'J', 10, 10);
INSERT INTO public.galaxy VALUES ('K', '11', 11, true, 'K', 11, 11);
INSERT INTO public.galaxy VALUES ('L', '12', 12, true, 'L', 12, 12);
INSERT INTO public.galaxy VALUES ('M', '13', 13, true, 'M', 13, 13);
INSERT INTO public.galaxy VALUES ('N', '14', 14, true, 'N', 14, 14);
INSERT INTO public.galaxy VALUES ('O', '15', 15, true, 'O', 15, 15);
INSERT INTO public.galaxy VALUES ('P', '16', 16, true, 'P', 16, 16);
INSERT INTO public.galaxy VALUES ('Q', '17', 17, true, 'Q', 17, 17);
INSERT INTO public.galaxy VALUES ('R', '18', 18, true, 'R', 18, 18);
INSERT INTO public.galaxy VALUES ('S', '19', 19, true, 'S', 19, 19);
INSERT INTO public.galaxy VALUES ('T', '20', 20, true, 'T', 20, 20);


--
-- Data for Name: moon; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.moon VALUES ('A', '1', '1', 1, true, '1', 1, 1);
INSERT INTO public.moon VALUES ('B', '2', '2', 2, true, '2', 2, 2);
INSERT INTO public.moon VALUES ('C', '3', '3', 3, true, '3', 3, 3);
INSERT INTO public.moon VALUES ('D', '4', '4', 4, true, '4', 4, 4);
INSERT INTO public.moon VALUES ('E', '5', '5', 5, true, '5', 5, 5);
INSERT INTO public.moon VALUES ('F', '6', '6', 6, true, '6', 6, 6);
INSERT INTO public.moon VALUES ('G', '7', '7', 7, true, '7', 7, 7);
INSERT INTO public.moon VALUES ('H', '8', '8', 8, true, '8', 8, 8);
INSERT INTO public.moon VALUES ('I', '9', '9', 9, true, '9', 9, 9);
INSERT INTO public.moon VALUES ('J', '10', '10', 10, true, '10', 10, 10);
INSERT INTO public.moon VALUES ('K', '11', '11', 11, true, '11', 11, 11);
INSERT INTO public.moon VALUES ('L', '12', '12', 12, true, '12', 12, 12);
INSERT INTO public.moon VALUES ('M', '13', '13', 13, true, '13', 13, 13);
INSERT INTO public.moon VALUES ('N', '14', '14', 14, true, '14', 14, 14);
INSERT INTO public.moon VALUES ('O', '15', '15', 15, true, '15', 15, 15);
INSERT INTO public.moon VALUES ('P', '16', '16', 16, true, '16', 16, 16);
INSERT INTO public.moon VALUES ('Q', '17', '17', 17, true, '17', 17, 17);
INSERT INTO public.moon VALUES ('R', '18', '18', 18, true, '18', 18, 18);
INSERT INTO public.moon VALUES ('S', '19', '19', 19, true, '19', 19, 19);
INSERT INTO public.moon VALUES ('T', '20', '20', 20, true, '20', 20, 20);


--
-- Data for Name: organism; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.organism VALUES ('A', '1', '1', 1, 1);
INSERT INTO public.organism VALUES ('B', '2', '2', 2, 2);
INSERT INTO public.organism VALUES ('C', '3', '3', 3, 3);


--
-- Data for Name: planet; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.planet VALUES ('A', '1', '1', true, '1', 1, 1);
INSERT INTO public.planet VALUES ('B', '2', '2', true, '2', 2, 2);
INSERT INTO public.planet VALUES ('C', '3', '3', true, '3', 3, 3);
INSERT INTO public.planet VALUES ('D', '4', '4', true, '4', 4, 4);
INSERT INTO public.planet VALUES ('E', '5', '5', true, '5', 5, 5);
INSERT INTO public.planet VALUES ('F', '6', '6', true, '6', 6, 6);
INSERT INTO public.planet VALUES ('G', '7', '7', true, '7', 7, 7);
INSERT INTO public.planet VALUES ('H', '8', '8', true, '8', 8, 8);
INSERT INTO public.planet VALUES ('I', '9', '9', true, '9', 9, 9);
INSERT INTO public.planet VALUES ('J', '10', '10', true, '10', 10, 10);
INSERT INTO public.planet VALUES ('K', '11', '11', true, '11', 11, 11);
INSERT INTO public.planet VALUES ('L', '12', '12', true, '12', 12, 12);
INSERT INTO public.planet VALUES ('M', '13', '13', true, '13', 13, 13);
INSERT INTO public.planet VALUES ('N', '14', '14', true, '14', 14, 14);
INSERT INTO public.planet VALUES ('O', '15', '15', true, '15', 15, 15);
INSERT INTO public.planet VALUES ('P', '16', '16', true, '16', 16, 16);
INSERT INTO public.planet VALUES ('Q', '17', '17', true, '17', 17, 17);
INSERT INTO public.planet VALUES ('R', '18', '18', true, '18', 18, 18);
INSERT INTO public.planet VALUES ('S', '19', '19', true, '19', 19, 19);
INSERT INTO public.planet VALUES ('T', '20', '20', true, '20', 20, 20);


--
-- Data for Name: star; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.star VALUES ('A', '1', '1', true, '1', 1, 1, 1);
INSERT INTO public.star VALUES ('B', '2', '2', true, '2', 2, 2, 2);
INSERT INTO public.star VALUES ('C', '3', '3', true, '3', 3, 3, 3);
INSERT INTO public.star VALUES ('D', '4', '4', true, '4', 4, 4, 4);
INSERT INTO public.star VALUES ('E', '5', '5', true, '5', 5, 5, 5);
INSERT INTO public.star VALUES ('F', '6', '6', true, '6', 6, 6, 6);
INSERT INTO public.star VALUES ('G', '7', '7', true, '7', 7, 7, 7);
INSERT INTO public.star VALUES ('H', '8', '8', true, '8', 8, 8, 8);
INSERT INTO public.star VALUES ('I', '9', '9', true, '9', 9, 9, 9);
INSERT INTO public.star VALUES ('J', '10', '10', true, '10', 10, 10, 10);
INSERT INTO public.star VALUES ('K', '11', '11', true, '11', 11, 11, 11);
INSERT INTO public.star VALUES ('L', '12', '12', true, '12', 12, 12, 12);
INSERT INTO public.star VALUES ('M', '13', '13', true, '13', 13, 13, 13);
INSERT INTO public.star VALUES ('N', '14', '14', true, '14', 14, 14, 14);
INSERT INTO public.star VALUES ('O', '15', '15', true, '15', 15, 15, 15);
INSERT INTO public.star VALUES ('P', '16', '16', true, '16', 16, 16, 16);
INSERT INTO public.star VALUES ('Q', '17', '17', true, '17', 17, 17, 17);
INSERT INTO public.star VALUES ('R', '18', '18', true, '18', 18, 18, 18);
INSERT INTO public.star VALUES ('S', '19', '19', true, '19', 19, 19, 19);
INSERT INTO public.star VALUES ('T', '20', '20', true, '20', 20, 20, 20);


--
-- Name: galaxy galaxy_has_life_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_has_life_key UNIQUE (has_life);


--
-- Name: galaxy galaxy_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_pkey PRIMARY KEY (galaxy_id);


--
-- Name: moon moon_has_life_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_has_life_key UNIQUE (has_life);


--
-- Name: moon moon_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_pkey PRIMARY KEY (moon_id);


--
-- Name: organism organism_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.organism
    ADD CONSTRAINT organism_pkey PRIMARY KEY (organism_id);


--
-- Name: organism organism_size_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.organism
    ADD CONSTRAINT organism_size_key UNIQUE (size);


--
-- Name: planet planet_has_life_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_has_life_key UNIQUE (has_life);


--
-- Name: planet planet_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_pkey PRIMARY KEY (planet_id);


--
-- Name: star star_has_life_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_has_life_key UNIQUE (has_life);


--
-- Name: star star_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_pkey PRIMARY KEY (star_id);


--
-- Name: moon moon_planet_id_fkey; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_planet_id_fkey FOREIGN KEY (planet_id) REFERENCES public.planet(planet_id);


--
-- Name: organism organism_moon_id_fkey; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.organism
    ADD CONSTRAINT organism_moon_id_fkey FOREIGN KEY (moon_id) REFERENCES public.moon(moon_id);


--
-- Name: planet planet_star_id_fkey; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_star_id_fkey FOREIGN KEY (star_id) REFERENCES public.star(star_id);


--
-- Name: star star_galaxy_id_fkey; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_galaxy_id_fkey FOREIGN KEY (galaxy_id) REFERENCES public.galaxy(galaxy_id);


--
-- PostgreSQL database dump complete
--

